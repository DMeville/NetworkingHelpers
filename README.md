# NetworkingHelpers
Networking helpers is a collection of helper classes for networked games. 
Based on work from various others, simply putting it together and improving their work. 
Much credit goes to Alexander Shoulson, Glenn Fiedler and Stanislav Denisov.

# BitBufferV2
A new version of BitBuffer, Faster and supporting bit level compression by ranged values. Quaternion compression, Float ranged compression and string UTF-16 support.


Important change to other bitbuffers is that you have to finalize the stream.
You fill the buffer with Add commands and if you are done you have to call the Finish() void. 
If you call ToArray or ToSpan it will automatically invoke the Finish.
