# $NetBSD: Makefile,v 1.6 2017/06/20 18:52:01 youri Exp $

PKGREVISION= 4
.include "../../meta-pkgs/xfce4/Makefile.common"

DISTNAME=	thunar-media-tags-plugin-0.2.1
PKGNAME=	xfce4-${DISTNAME}
CATEGORIES=	multimedia
MASTER_SITES=	http://archive.xfce.org/src/thunar-plugins/thunar-media-tags-plugin/0.2/

MAINTAINER=	gls@NetBSD.org
HOMEPAGE=	http://goodies.xfce.org/projects/thunar-plugins/thunar-media-tags-plugin
COMMENT=	Thunar media tags plugin

.include "../../audio/taglib/buildlink3.mk"
.include "../../x11/gtk2/buildlink3.mk"
.include "../../x11/xfce4-exo/buildlink3.mk"
.include "../../sysutils/xfce4-thunar/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
