# Created by: Andrey Zakhvatov
# $FreeBSD$

PORTNAME=	xdigger
PORTVERSION=	1.0.10
PORTREVISION=	3
CATEGORIES=	games
MASTER_SITES=	SUNSITE/games/arcade

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Boulderdash-like KC85 Digger for X Window System

USES=		imake tar:tgz
USE_XORG=	x11 xext

DESKTOP_ENTRIES="XDigger" "" "" "${PORTNAME}" "" ""

OPTIONS_DEFINE=	DOCS

post-patch:
	@${REINPLACE_CMD} -e "s|%%PREFIX%%|${PREFIX}|g" ${WRKSRC}/configure.h

post-install:
	@${MKDIR} ${STAGEDIR}${DOCSDIR}
.for i in ChangeLog README
	(cd ${WRKSRC} && ${INSTALL_DATA} ${i} ${STAGEDIR}${DOCSDIR})
.endfor

.include <bsd.port.mk>
