INCFLAGS=-I. -I../include

FLTFLAGS="-s 1331200"   
export FLTFLAGS
#CFLAGS=-w -O3 -g $(INCFLAGS)
#CHOST="i686-pc-linux-gnu"
#CFLAGS=-fprefetch-loop-arrays -march=pentium4 -w -O3 -pipe -fomit-frame-pointer -freg-struct-return -malign-double -maccumulate-outgoing-args -minline-all-stringops -mmmx -msse -msse2 $(INCFLAGS)
CFLAGS=-fprefetch-loop-arrays -march=native -w -O3 -pipe -fomit-frame-pointer -freg-struct-return -malign-double -maccumulate-outgoing-args -minline-all-stringops -mmmx -msse -msse2 $(INCFLAGS)
#CXXFLAGS="-march=pentium4 -O3 -pipe -fomit-frame-pointer"

PROG=libmagic.a

SRC=magic.c magic_base.c magic_field.c
OBJ=$(SRC:.c=.o)


ifeq (0,$(MAKELEVEL))
CC=gcc
RM=rm -f
AR=ar cr
MV=mv
RANLIB=ranlib
SED=sed
SHELL=/bin/sh
endif

all: $(PROG)
$(PROG): $(OBJ)
	$(RM) $(PROG)
	$(AR) $(PROG) $(OBJ)
	$(RANLIB) $(PROG)

depend:
	$(MV) Makefile Makefile.bak
	$(SED) -ne '1,/^# DO NOT DELETE THIS LINE/p' Makefile.bak>Makefile
	$(CC) $(INCFLAGS) -M $(SRC) >> Makefile 

clean:
	$(RM) $(PROG)
	$(RM) $(OBJ)
	$(RM) *~

distclean:
	$(RM) $(PROG)
	$(RM) $(OBJ)
	$(RM) *~
	$(MV) Makefile Makefile.bak
	$(SED) -ne '1,/^# DO NOT DELETE THIS LINE/p' Makefile.bak>Makefile
	$(RM) Makefile.bak

# DO NOT DELETE THIS LINE
magic.o: magic.c ../include/version.h ../include/correct_bug.h \
  ../include/version_pk.h /usr/include/stdio.h /usr/include/features.h \
  /usr/include/sys/cdefs.h /usr/include/gnu/stubs.h \
  /usr/lib/gcc-lib/i386-redhat-linux/3.2.2/include/stddef.h \
  /usr/include/bits/types.h /usr/include/bits/wordsize.h \
  /usr/include/bits/typesizes.h /usr/include/libio.h \
  /usr/include/_G_config.h /usr/include/wchar.h /usr/include/bits/wchar.h \
  /usr/include/gconv.h \
  /usr/lib/gcc-lib/i386-redhat-linux/3.2.2/include/stdarg.h \
  /usr/include/bits/stdio_lim.h /usr/include/bits/sys_errlist.h \
  /usr/include/string.h ../include/common.h /usr/include/errno.h \
  /usr/include/bits/errno.h /usr/include/linux/errno.h \
  /usr/include/asm/errno.h ../include/char_base.h ../include/skill.h \
  ../include/util.h /usr/include/sys/time.h /usr/include/time.h \
  /usr/include/bits/time.h /usr/include/sys/select.h \
  /usr/include/bits/select.h /usr/include/bits/sigset.h \
  /usr/include/stdlib.h /usr/include/sys/types.h /usr/include/endian.h \
  /usr/include/bits/endian.h /usr/include/sys/sysmacros.h \
  /usr/include/bits/pthreadtypes.h /usr/include/bits/sched.h \
  /usr/include/alloca.h ../include/title.h ../include/addressbook.h \
  ../include/net.h /usr/include/netinet/in.h /usr/include/stdint.h \
  /usr/include/bits/socket.h \
  /usr/lib/gcc-lib/i386-redhat-linux/3.2.2/include/limits.h \
  /usr/lib/gcc-lib/i386-redhat-linux/3.2.2/include/syslimits.h \
  /usr/include/limits.h /usr/include/bits/posix1_lim.h \
  /usr/include/bits/local_lim.h /usr/include/linux/limits.h \
  /usr/include/bits/posix2_lim.h /usr/include/bits/sockaddr.h \
  /usr/include/asm/socket.h /usr/include/asm/sockios.h \
  /usr/include/bits/in.h /usr/include/bits/byteswap.h \
  /usr/include/signal.h /usr/include/bits/signum.h \
  /usr/include/bits/siginfo.h /usr/include/bits/sigaction.h \
  /usr/include/bits/sigcontext.h /usr/include/asm/sigcontext.h \
  /usr/include/bits/sigstack.h /usr/include/bits/sigthread.h \
  /usr/include/pthread.h /usr/include/sched.h \
  /usr/include/bits/initspin.h ../include/link.h ../include/char_data.h \
  ../include/item.h ../include/char.h ../include/battle.h \
  ../include/magic_base.h ../include/magic.h ../include/magic_field.h \
  ../include/family.h ../include/handletime.h ../include/battle_magic.h \
  ../include/battle_event.h ../include/lssproto_serv.h \
  ../include/lssproto_util.h /usr/include/strings.h /usr/include/unistd.h \
  /usr/include/bits/posix_opt.h /usr/include/bits/confname.h \
  /usr/include/getopt.h ../include/pet_skill.h
magic_base.o: magic_base.c ../include/version.h ../include/correct_bug.h \
  ../include/version_pk.h /usr/include/stdio.h /usr/include/features.h \
  /usr/include/sys/cdefs.h /usr/include/gnu/stubs.h \
  /usr/lib/gcc-lib/i386-redhat-linux/3.2.2/include/stddef.h \
  /usr/include/bits/types.h /usr/include/bits/wordsize.h \
  /usr/include/bits/typesizes.h /usr/include/libio.h \
  /usr/include/_G_config.h /usr/include/wchar.h /usr/include/bits/wchar.h \
  /usr/include/gconv.h \
  /usr/lib/gcc-lib/i386-redhat-linux/3.2.2/include/stdarg.h \
  /usr/include/bits/stdio_lim.h /usr/include/bits/sys_errlist.h \
  /usr/include/string.h ../include/common.h /usr/include/errno.h \
  /usr/include/bits/errno.h /usr/include/linux/errno.h \
  /usr/include/asm/errno.h ../include/buf.h ../include/configfile.h \
  ../include/magic_base.h ../include/util.h /usr/include/sys/time.h \
  /usr/include/time.h /usr/include/bits/time.h /usr/include/sys/select.h \
  /usr/include/bits/select.h /usr/include/bits/sigset.h \
  /usr/include/stdlib.h /usr/include/sys/types.h /usr/include/endian.h \
  /usr/include/bits/endian.h /usr/include/sys/sysmacros.h \
  /usr/include/bits/pthreadtypes.h /usr/include/bits/sched.h \
  /usr/include/alloca.h ../include/magic.h
magic_field.o: magic_field.c ../include/version.h \
  ../include/correct_bug.h ../include/version_pk.h /usr/include/stdio.h \
  /usr/include/features.h /usr/include/sys/cdefs.h \
  /usr/include/gnu/stubs.h \
  /usr/lib/gcc-lib/i386-redhat-linux/3.2.2/include/stddef.h \
  /usr/include/bits/types.h /usr/include/bits/wordsize.h \
  /usr/include/bits/typesizes.h /usr/include/libio.h \
  /usr/include/_G_config.h /usr/include/wchar.h /usr/include/bits/wchar.h \
  /usr/include/gconv.h \
  /usr/lib/gcc-lib/i386-redhat-linux/3.2.2/include/stdarg.h \
  /usr/include/bits/stdio_lim.h /usr/include/bits/sys_errlist.h \
  ../include/common.h /usr/include/errno.h /usr/include/bits/errno.h \
  /usr/include/linux/errno.h /usr/include/asm/errno.h \
  ../include/char_base.h ../include/skill.h ../include/util.h \
  /usr/include/sys/time.h /usr/include/time.h /usr/include/bits/time.h \
  /usr/include/sys/select.h /usr/include/bits/select.h \
  /usr/include/bits/sigset.h /usr/include/stdlib.h \
  /usr/include/sys/types.h /usr/include/endian.h \
  /usr/include/bits/endian.h /usr/include/sys/sysmacros.h \
  /usr/include/bits/pthreadtypes.h /usr/include/bits/sched.h \
  /usr/include/alloca.h ../include/title.h ../include/addressbook.h \
  ../include/net.h /usr/include/netinet/in.h /usr/include/stdint.h \
  /usr/include/bits/socket.h \
  /usr/lib/gcc-lib/i386-redhat-linux/3.2.2/include/limits.h \
  /usr/lib/gcc-lib/i386-redhat-linux/3.2.2/include/syslimits.h \
  /usr/include/limits.h /usr/include/bits/posix1_lim.h \
  /usr/include/bits/local_lim.h /usr/include/linux/limits.h \
  /usr/include/bits/posix2_lim.h /usr/include/bits/sockaddr.h \
  /usr/include/asm/socket.h /usr/include/asm/sockios.h \
  /usr/include/bits/in.h /usr/include/bits/byteswap.h \
  /usr/include/signal.h /usr/include/bits/signum.h \
  /usr/include/bits/siginfo.h /usr/include/bits/sigaction.h \
  /usr/include/bits/sigcontext.h /usr/include/asm/sigcontext.h \
  /usr/include/bits/sigstack.h /usr/include/bits/sigthread.h \
  /usr/include/pthread.h /usr/include/sched.h \
  /usr/include/bits/initspin.h ../include/link.h ../include/char.h \
  ../include/char_data.h ../include/item.h ../include/magic_base.h \
  ../include/magic.h ../include/magic_field.h
