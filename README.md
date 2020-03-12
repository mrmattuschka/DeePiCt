# tomo-organelle-detection
### TODO:
- Envs
- CLI Documentation
- Replace EMAN2 with proprietary filter module (EMAN2 comes with its own python, causing issues)
- Merge filtering methods again?
- Fix Y flipping in predictions
- DONE Proper defaults
- DONE Decide whether to re-run on config changes -> nope, has to be forced by the user now.
- DONE remove normalization step from training scripts
- DONE Filtering
- DONE z_stride fix
- DONE flip_y as CLI arg
- DONE prediction module
- DONE crop compensation
- DONE output loc management (also for intermediates)


Check Transfer learning
Include membrane data?
    -> Only viable if membranes are detected reliably (my Unet works quite well if the membranes are easily distinguishable)
Label pooling script
    -> for Cytosol detection
    remove Label preprocessing in training scripts 
