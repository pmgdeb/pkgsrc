# $NetBSD: Makefile,v 1.30 2017/02/12 06:25:36 ryoon Exp $
#

DISTNAME=		scim-ccinput-0.3.1
PKGREVISION=		25
CATEGORIES=		inputmethod chinese
MASTER_SITES=		${MASTER_SITE_SOURCEFORGE:=scim/}
EXTRACT_SUFX=		.tar.bz2

MAINTAINER=		pkgsrc-users@NetBSD.org
HOMEPAGE=		http://www.scim-im.org/
COMMENT=		SCIM IMEngine module for CCInput
LICENSE=		gnu-gpl-v2

GNU_CONFIGURE=		yes
USE_LIBTOOL=		yes
USE_PKGLOCALEDIR=	yes
USE_LANGUAGES=		c c++
USE_TOOLS+=		pkg-config bash msgfmt
CONFIG_SHELL=		${BASH}

USE_SCIM_GTKUTILS=	yes

SUBST_CLASSES+=		localedir
SUBST_STAGE.localedir=	pre-configure
SUBST_SED.localedir+=	-e 's,\$$(datadir)/locale,@prefix@/${PKGLOCALEDIR}/locale,'
SUBST_SED.localedir+=	-e 's,/usr/share/locale,${PREFIX}/${PKGLOCALEDIR}/locale,'
SUBST_FILES.localedir=	po/Makefile.am po/Makefile.in
SUBST_FILES.localedir+= scim/IMEngine/scim_ccin_imengine.cpp
SUBST_FILES.localedir+=	scim/SetupUI/scim_ccin_imengine_setup.cpp

.include "../../devel/gettext-lib/buildlink3.mk"
.include "../../inputmethod/scim/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
