# $NetBSD: Makefile,v 1.20 2018/08/22 09:47:28 wiz Exp $

DISTNAME=	Apache-AuthCookie-3.27
PKGNAME=	p5-${DISTNAME:S/Apache/Apache2/}
PKGREVISION=	1
CATEGORIES=	www perl5
MASTER_SITES=	http://search.cpan.org/CPAN/authors/id/M/MS/MSCHOUT/

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://search.cpan.org/dist/Apache-AuthCookie/
COMMENT=	Perl5 module for Authentication and Authorization via cookies
LICENSE=	${PERL5_LICENSE}

DEPENDS+=	p5-Class-Load-[0-9]*:../../devel/p5-Class-Load
DEPENDS+=	p5-URI-[0-9]*:../../www/p5-URI
DEPENDS+=	p5-libwww-[0-9]*:../../www/p5-libwww

PERL5_PACKLIST=		auto/Apache/AuthCookie/.packlist

.include "../../lang/perl5/module.mk"
.include "../../www/ap2-perl/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
