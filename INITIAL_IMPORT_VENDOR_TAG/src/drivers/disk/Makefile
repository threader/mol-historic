
include			../../../config/Makefile.top

XTARGETS		= disk
disk-OBJS		= blkdev.o disk_open.o ablk.o pseudofs.o \
			  scsi.o $(dbg-y) $(obj-scsi-y)

obj-scsi-$(LINUX)	= sg-scsi.o cd-scsi.o ablk-cd.o
dbg-$(CONFIG_SCSIDEBUG)	= scsidbg.o

INCLUDES		= -I../include

include			$(rules)/Rules.make
