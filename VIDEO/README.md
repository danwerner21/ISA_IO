F8000 - window
3e0 - SID


;;; 	VRAM Memory Map
;;;	$1000-$177F	40/80 Text Page 1
;;;	$1800-$1F7F	40/80 Color Page 1
;;;	$2000-$277F	40/80 Text Page 2
;;;	$2800-$2F7F	40/80 Color Page 2
;;;	$2000-$5FFF	HIRES PAGE 1
;;;	$6000-$8FFF	HIRES PAGE 2
;;;	$2000-$BFFF	DOUBLE HIRES

  $0x00 0x01=soft_scanline_emulation, 0x02 nO soft_scanline_emulatioN
  $0x01 0x01=page1, 0x02 page2
  $0x02  character generator write offset (data << 3)
  $0x03 character generator write DATA
  $0x04 EXECUTE device command
        0x00- reset to the default configuration
        0x01- reset to the saved configuration
	0x02- save the current configuration

  $0x05  0x01=soft_text=true, 0x02=soft_text=false
  $0x06 Lores Mode=0X01,NO lores Mode=0x02
  $0x07 Double Lores Mode=0X01,NO Double lores Mode=0x02
  $0x08 Hires Mode=0X01,NO Hires Mode=0x02
  $0x09 Double Hires Mode=0X01,NO Double Hires lores Mode=0x02
  $0x0A 80COL Mode=0X01,NO 80COL Mode=0x02
  $0x0B MIXED Mode=0X01,NO MIXED Mode=0x02
  $0x0C QUAD Hires Mode=0X01,NO QUAD Hires lores Mode=0x02
  $0x0D MONO Hires Mode=0X01,NO MONO Hires lores Mode=0x02
 


>EFE2 00
>EFE1 03
>EFD0 00 01 02 03 04 05 06 07
>EFD8 F8 F9 FA FB 0C 0D 0E 0F
>EFE0 03
>EFE2 01

>9000 65 66 67 68 69 70 71 72
>9800 12 13 32 23 43 45 54 31
