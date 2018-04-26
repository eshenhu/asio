# asio
Asio C++ Library

Add some addtional features:

1. add async_receive_with_tmo(...), async_receive_from_with_tmo(...)
      The reason is sometimes the message was expected to received with the wanted time duration. The ordinary method is start
      a timer to count-down the tick, but it is not handful in the coding. The added method will be triggered on the same 
      handler with the receiving handler but with the special error code indicating tmo.
