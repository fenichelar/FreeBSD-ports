PORTNAME=	kdiff3
DISTVERSION=	1.11.5
CATEGORIES=	textproc kde
MASTER_SITES=	KDE/stable/${PORTNAME}

MAINTAINER=	kde@FreeBSD.org
COMMENT=	KDE graphical frontend for diff
WWW=		https://kdiff3.sourceforge.net/

LICENSE=	GPLv2
LICENSE_FILE=	${WRKSRC}/COPYING

BUILD_DEPENDS=	${LOCALBASE}/include/boost/range/algorithm.hpp:devel/boost-libs

USES=		cmake compiler:c++11-lang kde:5 qt:5 tar:xz xorg
USE_KDE=	auth codecs completion config configwidgets coreaddons crash \
		i18n jobwidgets kio service solid widgetsaddons windowsystem \
		xmlgui \
		doctools:build ecm:build
USE_QT=		concurrent core dbus gui network printsupport widgets xml \
		buildtools:build qmake:build
USE_XORG=	x11

DOCSDIR_REL=	share/doc/HTML

OPTIONS_DEFINE=	DOCS

.include <bsd.port.mk>
