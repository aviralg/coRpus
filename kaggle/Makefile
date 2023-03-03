KERNEL_INFO_WEBPAGES_DIRPATH := kernel-info-webpages
KERNEL_INFO_FILEPATH := kernel-info.csv
PART_COUNT := 2700
PART_INDEX := 1
KERNEL_CODE_DOWNLOAD_DELAY := 30
KERNEL_DIRPATH := kernels
KERNEL_CODE_DOWNLOAD_STATUS_FILEPATH := kernel-code-download-status.csv


extract-kernel-info:
	/mnt/nvme0/aviral/R-dyntrace/bin/R --slave --file=extract-kernel-info --args $(KERNEL_INFO_WEBPAGES_DIRPATH) $(KERNEL_INFO_FILEPATH)


download-kernel-code:
	/mnt/nvme0/aviral/R-dyntrace/bin/R --slave --file=download-kernel-code --args $(KERNEL_INFO_FILEPATH) $(PART_COUNT) $(PART_INDEX) $(KERNEL_CODE_DOWNLOAD_DELAY) $(KERNEL_DIRPATH) $(KERNEL_CODE_DOWNLOAD_STATUS_FILEPATH)


.PHONY: extract-kernel-info  \
        download-kernel-code
