KERNEL_INFO_WEBPAGES_DIRPATH := kernel-info-webpages
KERNEL_INFO_FILEPATH := kernel-info.csv
PART_COUNT := 2700
PART_INDEX := 1
KERNEL_CODE_DOWNLOAD_DELAY := 30
KERNEL_DIRPATH := kernels
KERNEL_CODE_DOWNLOAD_STATUS_FILEPATH := kernel-code-download-status.csv


extract-kernel-info:
	./extract-kernel-info $(KERNEL_INFO_WEBPAGES_DIRPATH) $(KERNEL_INFO_FILEPATH)


download-kernel-code:
	./download-kernel-code $(KERNEL_INFO_FILEPATH) $(PART_COUNT) $(PART_INDEX) $(KERNEL_CODE_DOWNLOAD_DELAY) $(KERNEL_DIRPATH) $(KERNEL_CODE_DOWNLOAD_STATUS_FILEPATH)


.PHONY: extract-kernel-info  \
        download-kernel-code
