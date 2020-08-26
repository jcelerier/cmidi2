# cmidi2: tiny MIDI 2.0 UMP processor library

This is a tiny library to process MIDI 2.0 UMP (Universal MIDI Packet).

MIDI 2.0 is designed to be allocation free by defining every message in 32bit,
64bit, or 128bit packet, including sysex messages.
This library populates those packets simply in integer values.
It should be usable within realtime audio applications.

As of v0.1, every function is static inline (if you are familiar with [LV2](lv2plug.in/) you would notice that this implementation style is quite simiar to it).

No commented documentation yet, but API reference can be generated by doxygen
and the first published version is available at https://cmidi2-api.web.app/reference/


