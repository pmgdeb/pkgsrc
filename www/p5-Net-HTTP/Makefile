# $NetBSD: Makefile,v 1.22 2017/06/14 13:31:16 wiz Exp $

DISTNAME=	Net-HTTP-6.16
PKGNAME=	p5-${DISTNAME}
CATEGORIES=	www perl5 net
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=Net/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://search.cpan.org/dist/Net-HTTP/
COMMENT=	Perl 5 module for low-level HTTP connections (client)
LICENSE=	${PERL5_LICENSE}

# TEST_DEPENDS
BUILD_DEPENDS+=	p5-URI-[0-9]*:../../www/p5-URI

USE_LANGUAGES=	# empty
PERL5_PACKLIST= auto/Net/HTTP/.packlist

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
