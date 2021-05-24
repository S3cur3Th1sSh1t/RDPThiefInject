# RDPThiefInject

Today I read the following article:

* [https://pentestlab.blog/2021/05/24/dumping-rdp-credentials/](https://pentestlab.blog/2021/05/24/dumping-rdp-credentials/)

And I thought why converting RDPThief into csharp, when the DLL can be converted to position independent shellcode via donut and injected via good old classic CreateRemoteThread? So, this repo does this as PoC. Conversion to Syscalls is easy at this point as all things needed are public and up to the reader.

Credit goes to [donut](https://github.com/TheWover/donut) && [RdpThief](https://github.com/0x09AL/RdpThief).

The credentials are put into the default RDPThief directory `C:\users\username\appdata\local\temp\data.bin` - no code modifications at all here.
