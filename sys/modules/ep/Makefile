# $FreeBSD$

.include <bsd.own.mk>

.PATH: ${.CURDIR}/../../dev/ep

KMOD=	if_ep
SRCS=	if_ep.c
SRCS+=	if_ep_pccard.c pccarddevs.h card_if.h
SRCS+=	if_ep_isa.c isa_if.h
.if ${MK_EISA} != "no"
SRCS+=	if_ep_eisa.c eisa_if.h
.endif
#SRCS+=	if_ep_mca.c
SRCS+=	bus_if.h device_if.h

.include <bsd.kmod.mk>
