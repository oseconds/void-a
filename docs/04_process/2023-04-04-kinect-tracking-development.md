# 2023.04.04 Kinect Tracking Development

## Context

After exploring real-time trompe-l'œil and viewpoint-dependent anamorphic rendering,
the next challenge was obtaining the viewer's viewpoint in physical space.

## Research

Kinect was investigated as a method for:

- detecting viewer position
- estimating viewing direction
- connecting physical location to virtual camera position

Research topics:

- Kinect sensing range
- depth camera limitations
- installation distance
- tracking stability
- real-time data transmission


## Conceptual Relation

The tracking system was not intended as a visible interaction device.

The purpose was to create an invisible relationship where:

viewer position
→
virtual viewpoint change
→
object appears to perceive the viewer


## Development Direction

Physical observer position becomes a parameter of the virtual camera,
allowing the artwork to respond to the viewer's presence without explicit control.