# $NetBSD: Makefile,v 1.7 2018/02/26 10:55:46 adam Exp $

DISTNAME=	Unidecode-1.0.22
PKGNAME=	${PYPKGPREFIX}-${DISTNAME}
CATEGORIES=	textproc python
MASTER_SITES=	${MASTER_SITE_PYPI:=U/Unidecode/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://github.com/avian2/unidecode
COMMENT=	ASCII transliterations of Unicode text
LICENSE=	gnu-gpl-v2

USE_LANGUAGES=	# none

post-install:
	cd ${DESTDIR}${PREFIX}/bin && ${MV} unidecode unidecode${PYVERSSUFFIX} || ${TRUE}

.include "../../lang/python/egg.mk"
.include "../../mk/bsd.pkg.mk"
