PACKAGE=ssh
LIB=	fido2
PRIVATELIB=
DIST=	${SRCTOP}/contrib/libfido2

.PATH:	${DIST}/src ${DIST}

SRCS+=	aes256.c
SRCS+=	assert.c
SRCS+=	authkey.c
SRCS+=	bio.c
SRCS+=	blob.c
SRCS+=	buf.c
SRCS+=	cbor.c
SRCS+=	compress.c
SRCS+=	config.c
SRCS+=	cred.c
SRCS+=	credman.c
SRCS+=	dev.c
SRCS+=	ecdh.c
SRCS+=	eddsa.c
SRCS+=	err.c
SRCS+=	es256.c
SRCS+=	es384.c
SRCS+=	hid_freebsd.c
SRCS+=	hid_unix.c
SRCS+=	hid.c
SRCS+=	info.c
SRCS+=	io.c
SRCS+=	iso7816.c
SRCS+=	largeblob.c
SRCS+=	log.c
SRCS+=	pin.c
SRCS+=	random.c
SRCS+=	reset.c
SRCS+=	rs1.c
SRCS+=	rs256.c
SRCS+=	time.c
SRCS+=	touch.c
SRCS+=	tpm.c
SRCS+=	types.c
SRCS+=	u2f.c
SRCS+=	util.c

SRCS+=	openbsd-compat/freezero.c
SRCS+=	openbsd-compat/recallocarray.c

CFLAGS+= -I ${DIST}/src -I${SRCTOP}/contrib/libcbor/src -I${.CURDIR}/../libcbor
CFLAGS+= -D_FIDO_INTERNAL
CFLAGS+= -DHAVE_ARC4RANDOM_BUF
CFLAGS+= -DHAVE_ASPRINTF
CFLAGS+= -DHAVE_CLOCK_GETTIME
CFLAGS+= -DHAVE_DEV_URANDOM
CFLAGS+= -DHAVE_ERR_H
CFLAGS+= -DHAVE_EXPLICIT_BZERO
CFLAGS+= -DHAVE_GETLINE
CFLAGS+= -DHAVE_GETOPT
CFLAGS+= -DHAVE_GETPAGESIZE
CFLAGS+= -DHAVE_GETRANDOM
CFLAGS+= -DHAVE_OPENSSLV_H
CFLAGS+= -DHAVE_READPASSPHRASE
CFLAGS+= -DHAVE_SIGNAL_H
CFLAGS+= -DHAVE_STRLCAT
CFLAGS+= -DHAVE_STRLCPY
CFLAGS+= -DHAVE_STRSEP
CFLAGS+= -DHAVE_SYSCONF
CFLAGS+= -DHAVE_SYS_RANDOM_H
CFLAGS+= -DHAVE_TIMESPECSUB
CFLAGS+= -DHAVE_TIMINGSAFE_BCMP
CFLAGS+= -DHAVE_UNISTD_H
CFLAGS+= -DTLS=__thread
CFLAGS+= -D_FIDO_MAJOR=1
CFLAGS+= -D_FIDO_MINOR=13
CFLAGS+= -D_FIDO_PATCH=0

LIBADD=	crypto z

WARNS=2
MAN=

.include <bsd.lib.mk>
