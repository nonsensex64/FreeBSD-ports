# Created by: Torsten Zuhlsdorff <ports@toco-domains.de>
# $FreeBSD$

PORTNAME=	devise-two-factor
PORTVERSION=	2.1.0
CATEGORIES=	security rubygems
MASTER_SITES=	RG

MAINTAINER=	ruby@FreeBSD.org
COMMENT=	Barebones two-factor authentication with Devise

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

RUN_DEPENDS=	rubygem-activesupport4>=0:devel/rubygem-activesupport4 \
		rubygem-attr_encrypted>=1.3:security/rubygem-attr_encrypted \
		rubygem-devise-rails4>=3.5:devel/rubygem-devise-rails4 \
		rubygem-railties4>=0:www/rubygem-railties4 \
		rubygem-rotp>=2.0:devel/rubygem-rotp

NO_ARCH=	yes
USE_RUBY=	yes
USES=		gem

.include <bsd.port.mk>
