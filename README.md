To build:
 cd src

 make clean; make all

To test:
  cd examples

  cd ST

  ./testST.sh

  cd ../MT

  ./testMT.sh

About:
pinball2elf is a tool to create stand-alone Linux binaries from checkpoints for arbitrary portions of execution of other Linux programs . The checkpoints it converts are called ‘pinballs’ and they are generated by “Program Record Replay Toolkit” (aka PinPlay kit) that is available at www.pinplay.org.

To create ELF binary from PINBALL, run following command:

   pinball2elf -d <pinball.global.log> -s <pinball.0.reg> -m <pinball.text> -r <pinball.address> -x elf_binary_name

See examples/\*/test\*.sh scripts for example usage.
