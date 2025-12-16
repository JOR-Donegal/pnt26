# Information Theory
Claude Shannon was arguably one of the most significant engineers in the field of digital circuit design. However, he is more remembered for his contributions to information theory from 1948 [1]. Shannon wanted to know how much information could be passed across a channel, in theory. Shannon stated that “The fundamental problem of communication is that of reproducing a message sent from one point, either exactly or approximately, to another point” In Shannon’s models we have:

1. An information source or Sender that produces a message
2. A Transmitter (TX) which creates encodes a signal to be sent through a channel
3. Information that composes the message
4. A Channel, the medium over which the signal is transmitted
5. Noise, background noises in the channel for an audio signal, electrical noise in the channel for an electrical signal.
6. A Receiver (RX), which decodes the signal back into the message, a destination, for which the message is intended.

Changing the characteristics of any of the terms above determines how much information can pass through a channel. Everything in the universe can be described in terms of bits, information theory was ground-breaking for a range of areas in physics.

Although not the originator of the term, Shannon also defined the bit as a unit of information. Flip a fair coin, you have a single bit of information (heads/tails). Consider an unfair coin that will land only on heads, each flip provides zero information. If an unfair coin lands on heads 2/3 of the time, the information in each flip is 0.92 bits.

If you have dice at home, there are 2.7 bits of information per throw (on average, how many guesses you would have to make to figure out what number I threw). In information theory, you can have fractions of bits! The more you know about something, the less random it seems and therefore the less information per result. True randomness has the highest possible information content.

Shannon defined information entropy to measure the information content in a message, and the measure of uncertainty in the message. All this applies widely, for example to natural language.

If you compress a file of predictable information (all white) it will be tiny. If you compress a file of truly random data (white noise), the compressed file will be about the same size as the uncompressed file.

As an example, consider the two lines below.

- [AB, AB, AB, AB, AB, AB, AB, AB, AB, AB, AB, AB, AB, AB, AB, AB]
- [AB] * 16

They both contain the same information; one can be communicated much more efficiently that the other. The first will compress well, the second will not. If you are interested in this, do some background reading on LZW compression [2].  

[1] Shannon, C.E., 2001. A mathematical theory of communication. ACM SIGMOBILE mobile computing and communications review, 5(1), pp.3-55.

[2] Welch, T.A., 1984. A technique for high-performance data compression. Computer, 17(06), pp.8-19.