# cmidi2: header-only MIDI 2.0 UMP and MIDI-CI binary processor library

This is a small header-only library to process MIDI 2.0 UMP (Universal MIDI Packet)
and MIDI-CI system exclusive packets.

MIDI 2.0 is designed to be allocation free by defining every message in 32bit,
64bit, or 128bit packet, including sysex messages.
This library populates those packets simply in integer values.
It should be usable within realtime audio applications.

As of v0.3.4, every function is static inline (if you are familiar with [LV2](lv2plug.in/) you would notice that this implementation style is quite simiar to it, namely LV2 Atom).

No commented documentation yet, but API reference is generated by doxygen
and published every time we tag a release: https://atsushieno.github.io/cmidi2/

At this state I keep making **breaking changes** in the API.
If you use it then you should not expect any API/ABI stability at this state.

## Usages

[atsushieno/aap-core](https://github.com/atsushieno/aap-core/), [atsushieno/aap-lv2](https://github.com/atsushieno/aap-lv2), and [atsushieno/aap-juce](https://github.com/atsushieno/aap-juce) make use of this library.

[libremidi](https://github.com/jcelerier/libremidi) internally uses cmidi2 too.

## License

cmidi2 is distributed under the MIT License.
