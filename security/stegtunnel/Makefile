# $NetBSD: Makefile,v 1.6 2017/09/04 18:01:01 wiz Exp $

DISTNAME=	stegtunnel-0.4
PKGREVISION=	1
CATEGORIES=	security
#MASTER_SITES=	http://www.synacklabs.net/projects/stegtunnel/

MAINTAINER=	agc@NetBSD.org
#HOMEPAGE=	http://www.synacklabs.net/projects/stegtunnel/
COMMENT=	Provides a covert channel in the IPID and sequence number

GNU_CONFIGURE=	yes
USE_LIBTOOL=	yes

LIBS.SunOS+=	-lrt

.include "../../net/libdnet/buildlink3.mk"
.include "../../net/libpcap/buildlink3.mk"

.include "../../mk/bsd.pkg.mk"
