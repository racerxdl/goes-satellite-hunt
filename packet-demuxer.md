# Packet Demuxer

In the last chapter I showed how to get the frames from the demodulated bit stream. In this chapter I will show you how to parse these frames and get the packets that will on next chapter generate the files that GOES send. I will first add C code to the code I did in the last chapter to separated all the virtual channels by ID. But mainly this chapter will be done in python \(just because its easier, I will eventually make a C code as well to do the stuff\).

