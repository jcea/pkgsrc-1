# $NetBSD: Makefile,v 1.15 2018/04/13 16:31:09 tsutsui Exp $
#

DISTNAME=		cairo-gobject-${VERSION}
PKGNAME=		${RUBY_PKGPREFIX}-gnome2-${DISTNAME}
COMMENT=		Ruby binding of cairo-gobject
CATEGORIES=		graphics gnome

MAINTAINER=		tsutsui@NetBSD.org

DEPENDS+=		${RUBY_PKGPREFIX}-gnome2-glib>=${VERSION}:../../devel/ruby-gnome2-glib
DEPENDS+=		${RUBY_PKGPREFIX}-cairo>=1.14.3:../../graphics/ruby-cairo

.include "../../devel/ruby-gnome2-glib/buildlink3.mk"
.include "../../graphics/ruby-cairo/buildlink3.mk"
.include "../../graphics/cairo-gobject/buildlink3.mk"
.include "../../meta-pkgs/ruby-gnome2/Makefile.common"
.include "../../lang/ruby/gem.mk"
.include "../../mk/bsd.pkg.mk"
