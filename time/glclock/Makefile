# $NetBSD: Makefile,v 1.26 2018/07/18 00:06:24 joerg Exp $
#

DISTNAME=		glclock-6.0b6.0
PKGREVISION=		4
CATEGORIES=		x11 graphics time
MASTER_SITES=		http://www.daionet.gr.jp/~masa/archives/

MAINTAINER=		pkgsrc-users@NetBSD.org
HOMEPAGE=		http://www.daionet.gr.jp/~masa/glclock/
COMMENT=		OpenGL-based pocket watch

USE_LANGUAGES=		c++03

MAKE_FILE=		makefile
BUILD_TARGET=		glclock


.include "../../mk/bsd.prefs.mk"

.if ${OPSYS} == NetBSD && ${MACHINE_ARCH} == sparc
CFLAGS=
.endif

INSTALLATION_DIRS=	bin

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/glclock ${DESTDIR}${PREFIX}/bin
#notyet: lookup of .ppm files
#	for i in benchclock crystalclock marbleclock metalclock \
#			mwclock woodclock;do \
#	${INSTALL_SCRIPT} ${WRKSRC}/$$i ${PREFIX}/bin; done

.include "../../graphics/Mesa/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
