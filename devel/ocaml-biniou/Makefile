# $NetBSD: Makefile,v 1.9 2018/07/19 15:15:22 jaapb Exp $

GITHUB_PROJECT=	biniou
GITHUB_TAG=	v${PKGVERSION_NOREV}
DISTNAME=	${GITHUB_PROJECT}-1.2.0
PKGNAME=	ocaml-${DISTNAME}
PKGREVISION=	2
CATEGORIES=	devel
MASTER_SITES=	${MASTER_SITE_GITHUB:=mjambon/}

MAINTAINER=	jaapb@NetBSD.org
HOMEPAGE=	https://github.com/mjambon/biniou/
COMMENT=	Extensible binary data format, like JSON but faster
LICENSE=	modified-bsd

OCAML_USE_JBUILDER=	yes
INSTALLATION_DIRS+=	bin

.include "../../mk/ocaml.mk"

.if ${OCAML_USE_OPT_COMPILER} == "yes"
BUILD_TARGET+=	opt
.endif

.include "../../textproc/ocaml-easy-format/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
