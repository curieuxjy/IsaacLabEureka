# Note
- available envs: https://isaac-sim.github.io/IsaacLab/main/source/overview/environments.html

# Run
- `conda activate env_isaaclab`
- tasks: `./source/isaaclab_eureka/isaaclab_eureka/config/tasks.py`

```
# Cartpole
python scripts/train.py --task=Isaac-Cartpole-Direct-v0 --max_training_iterations=100 --rl_library="rl_games"

python scripts/play.py --task=Isaac-Cartpole-Direct-v0 --checkpoint=./logs/rl_runs/rl_games_eureka/cartpole_direct/2025-07-30_10-15-49_Run-0/nn/cartpole_direct.pth --num_envs=20 --rl_library="rl_games"

# Quadcopter
python scripts/train.py --task=Isaac-Quadcopter-Direct-v0 --max_training_iterations=200 --rl_library="rl_games"

python scripts/play.py --task=Isaac-Quadcopter-Direct-v0 --checkpoint=./logs/rl_runs/rl_games_eureka/quadcopter_direct/2025-07-30_13-52-06_Run-0/nn/quadcopter_direct.pth --num_envs=20 --rl_library="rl_games"
```
