# $NetBSD: Makefile,v 1.29 2017/06/05 14:23:49 ryoon Exp $
#

DISTNAME=	Tie-IxHash-1.23
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	3
CATEGORIES=	textproc perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=Tie/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://search.cpan.org/dist/Tie-IxHash/
COMMENT=	Perl module that implements ordered in-memory associative arrays
LICENSE=	${PERL5_LICENSE}

PERL5_PACKLIST=		auto/Tie/IxHash/.packlist
PERL5_MODULE_TYPE=	Module::Build

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
