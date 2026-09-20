Ambush Monster System
Hello! This is the Ambush Monster System—a complete, plug-and-play Unity package designed to handle patrolling jumpscare entities in 3D space.

What It Have
AmbushManager: Core controller script that handles movement, pathing logic, timings, and audio playback.
MonsterVisual: Child GameObject containing the monster model, a Kinematic Rigidbody, and a Box Collider set to Is Trigger.
AmbushCanvas: A World Space UI Canvas assigned directly to the camera to render jumpscare visuals in 3D space.
Dual-Audio Engine: Support for 2D incoming sounds, 3D spatialized proximity audio (100m max reach), and direct jumpscare impact audio.
AudioFixerTool Editor Utility: A custom toolbar script (Tools -> Fix All Scene Audio Issues) that scans and silences rogue Play On Awake settings across the scene.

What It Do
Patrols Waypoints: Moves between designated path points, waits at endpoints, and retraces its route in reverse.
Emits Dynamic 3D Audio: Scales proximity audio relative to the monster's distance from the player up to 100 meters.
Detects Player Touch: Listens for trigger and collision overlaps with the player via AmbushTouchCanvas.
Activates World Space Jumpscare: Instantly force-enables the World Space Canvas, activates child UI elements, and plays the jumpscare audio on contact.
Prevents Startup Glitches: Automatically stops audio sources and hides UI elements on scene load to prevent premature loops or accidental self-disabling.
