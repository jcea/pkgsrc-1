# $NetBSD: Makefile,v 1.2 2018/04/29 10:03:26 wiz Exp $

DISTNAME=	html5-parser-0.4.5
PKGNAME=	${PYPKGPREFIX}-${DISTNAME}
CATEGORIES=	textproc www python
MASTER_SITES=	${MASTER_SITE_PYPI:=h/html5-parser/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://github.com/kovidgoyal/html5-parser
COMMENT=	Fast, standards-compliant, C-based HTML5 parser
LICENSE=	apache-2.0

DEPENDS+=	${PYPKGPREFIX}-lxml-[0-9]*:../../textproc/py-lxml
DEPENDS+=	${PYPKGPREFIX}-beautifulsoup4-[0-9]*:../../www/py-beautifulsoup4

USE_TOOLS+=	pkg-config

.include "../../lang/python/egg.mk"
.include "../../textproc/libxml2/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
