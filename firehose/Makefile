NDK_BUILD:=/workspace/android-ndk/android-ndk-r10e/ndk-build

linux:
	$(CROSS_COMPILE)gcc -Wall -g -c qfirehose.c sahara_protocol.c firehose_protocol.c usb_linux_firehose.c -lpthread

android:
	$(NDK_BUILD) V=0 APP_BUILD_SCRIPT=Android.mk NDK_PROJECT_PATH=`pwd` NDK_DEBUG=0 APP_ABI='armeabi,arm64-v8a'

clean:
	rm -rf qfirehose obj libs *~
