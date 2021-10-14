# SSD-based Object Detection in PyTorch

This repo expands upon the work presented in [https://github.com/qfgaohao/pytorch-ssd](https://github.com/qfgaohao/pytorch-ssd) to provide the following:

## - Implementation of the `ReduceLROnPlateau` Learning Rate Scheduler
     - An additional LR scheduler to prevent overfitting
## - Inclusion of Optimizer `state_dict` in training checkpoint files
     - Facilitates the resumption of training sessions at previously-determined learning rates
## - Awareness of previous session epoch when using `resume` feature
     - Epoch numeration of checkpoint files for resumed sessions starts at the loaded checkpoint file's epoch value.
## - Generation of CSV loss reports for each training session
     - One epoch per row; includes learning rate, validation/regression/classification losses
