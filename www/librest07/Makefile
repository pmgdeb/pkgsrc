# $NetBSD: Makefile,v 1.22 2017/04/22 21:03:18 adam Exp $

DISTNAME=	rest-0.7.93
PKGNAME=	${DISTNAME:S/rest/librest07/}
PKGREVISION=	5
CATEGORIES=	www
MASTER_SITES=	${MASTER_SITE_GNOME:=sources/rest/0.7/}
EXTRACT_SUFX=	.tar.xz

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://wiki.gnome.org/Projects/Librest
COMMENT=	Library for "RESTful" web services
LICENSE=	gnu-lgpl-v2.1

GNU_CONFIGURE=	yes
USE_LIBTOOL=	yes
USE_TOOLS+=	pkg-config gmake
# see pkgsrc/security/mozilla-rootcerts
CONFIGURE_ARGS+= --with-ca-certificates=/etc/ssl/certs/ca-certificates.crt

PKGCONFIG_OVERRIDE+=	rest.pc.in rest-extras.pc.in

TEST_TARGET=	check

.include "options.mk"

.include "../../devel/glib2/buildlink3.mk"
.include "../../net/libsoup/buildlink3.mk"
.include "../../textproc/libxml2/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
