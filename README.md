Sat 25 Feb 17:14:05 UTC 2023

Please note:

   It is imperative, when trying to bring this system up on
   a target that has never run it before (or just not recently,
   with other firmware having been loaded most recently) ..

   It is imperative that all of the flash is erased, to run
   mecrisp-stellaris successfully.

   Otherwise a kind of boot loop situation arises.

   The system simply won't be useful if this simple precaution
   isn't taken.

   One solution: stm32f407 version of C.H. Ting's eForth v7.20 is
   a more tolerant firmware image than is mecrisp-stellaris.
   eForth can succsessfully be run on the stm32f407, and then used
   to erase all of flash space.

   That's a simple way to prepare the target's flash space for a
   subsequent firmware upload of mecrisp-stellaris.

   eForth (for stm32f4xx) can also be found in wa1tnr github.

   It will run as-is on stm32f407 Discovery, stm32f411 (Black Pill)
   and Adafruit stm32f405 express boards.

END.
