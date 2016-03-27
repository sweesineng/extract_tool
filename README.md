# extract_tool
Install device-tree-compiler
sudo apt-get install device-tree-compiler

Download split_bootimg.pl
sudo cp split_bootimg.pl /usr/local/bin
sudo chmod +x /usr/local/bin/split_bootimg.pl

Example:
split_bootimg.pl boot.img
  output:
  Page size: 2048 (0x00000800)
  Kernel size: 9593928 (0x00926448)
  Ramdisk size: 4915330 (0x004b0082)
  Second size: 0 (0x00000000)
  DT size: 2256896 (0x00227000)
  Board name: 
  Command line: console=null androidboot.hardware=qcom user_debug=31 msm_rtb.filter=0x37 dwc3_msm.cpu_to_affin=1
  ==================== 96 
  ==================== console=null androidboot.hardware=qcom user_debug=31 msm_rtb.filter=0x37 dwc3_msm.cpu_to_affin=1 
  Writing recovery.img-kernel ... complete.
  Writing recovery.img-ramdisk.gz ... complete.
  Writing recovery.img-dt.img ... complete.
