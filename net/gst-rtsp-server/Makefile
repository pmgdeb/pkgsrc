# $NetBSD: Makefile,v 1.4 2017/02/11 23:28:04 prlw1 Exp $

DISTNAME=	gst-rtsp-server-1.10.3
CATEGORIES=	net multimedia
MASTER_SITES=	http://gstreamer.freedesktop.org/src/gst-rtsp-server/
EXTRACT_SUFX=	.tar.xz

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://gstreamer.freedesktop.org/modules/gst-rtsp-server.html
COMMENT=	GStreamer RTSP server
LICENSE=	gnu-lgpl-v2

USE_LIBTOOL=		yes
GNU_CONFIGURE=		yes
USE_TOOLS+=		pkg-config gmake
PKGCONFIG_OVERRIDE=	gstreamer-rtsp-server.pc.in

BUILDLINK_API_DEPENDS.gstreamer1+=	gstreamer1>=1.10.0
.include "../../multimedia/gstreamer1/buildlink3.mk"
.include "../../multimedia/gst-plugins1-base/buildlink3.mk"
BUILDLINK_API_DEPENDS.glib2+=		glib2>=2.40.0
.include "../../devel/glib2/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
