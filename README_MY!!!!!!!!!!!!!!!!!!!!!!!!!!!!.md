screen
ssh -L 8111:localhost:8111 saion
srun -p test-gpu -c 8 -t 0-2:00:00 --gres=gpu:4 --mem-per-cpu=4G --pty bash
conda activate stylegan2pt
source $HOME/opt/gcc-7.1.0/activate
jupyter notebook --port 8111 --ip saion-gpu06.oist.jp --no-browser
open Project + Toonify + Interpolations - Train on Aliens OSMP

