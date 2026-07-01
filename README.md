# avlite-bridge-gazebo

Gazebo Ignition world bridge for AVLite. Registers `GazeboIgnitionBridge` — drives a Gazebo sim via ROS 2 topics.

## Install

```bash
git clone <this-repo> ~/.local/share/avlite/plugins/avlite-bridge-gazebo
```

Requires [AVLite](https://github.com/AV-Lab/avlite) and a running Gazebo Ignition instance with compatible ROS 2 interfaces.

## Configuration

```yaml
c40_community_plugins:
  avlite-bridge-gazebo: avlite-bridge-gazebo
c40_bridge: GazeboIgnitionBridge
```

Plugin settings: `~/.config/avlite/plugin_avlite-bridge-gazebo.yaml` (see `config/default.yaml`).

## Requirements

Source ROS 2 in your shell, then:

```bash
pip install -r requirements.txt
```

Ensure Gazebo and the bridge launch files are running before starting AVLite.
