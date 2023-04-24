

<b>RUn Guide</b>:
The AI has successfully completed 1-1, 2-1, 3-1, 4-1 but in our model failed to complete and still requires more training 5-1, 6-1, and 7-1.

## Installation guide
You will need Python 3.6 or newer.

1. `cd /path/to/SuperMarioBros-AI`
2. Run `pip install -r requirements.txt`
3. Install the ROM
   - Head on over to the ROM for [Super Mario Bros.](https://wowroms.com/en/roms/nintendo-entertainment-system/super-mario-bros./23755.html) and click `download`.
4. Unzip `Super Mario Bros. (World).zip` to some location
5. Run `python -m retro.import "/path/to/unzipped/super mario bros. (world)"`
    - Make sure you run this on the folder, i.e. `python -m retro.import "c:\Users\chris\Downloads\Super Mario Bros. (World)"`
    - You should see output text:
      ```
      Importing SuperMarioBros-Nes
      Imported 1 games
      ```
## Command Line Options
 `python smb_ai.py -h` run to see what commands you can use for the program.



### Loading Individuals
there multiple folders attached whatever folder you want to load you can use the following way to load them.
- `--load-file FOLDER`. Indicate the `/path/to/population/folder` that you want to load from.

Note that loading individuals only supports loading the best performing one from generations.

### Replaying Individuals
This is helpful if you want to watch particular individuals replay their run. You must specify *both* of the below arguments:
- `--replay-file FOLDER`. Indicate the `/path/to/population/folder` that you want to replay from.
- `--replay-inds INDS`. This accepts the same syntax as `--load-inds` with one additional syntax. If you want to replay starting at a certain individual through the end of the folder, you can do `[12,]` and this will begin at `best_ind_gen12` and run through the entire folder. *NOTE*: this is not supported in `--load-inds` since when you load it will be treated as an initially population and those individuals will be treated as parents. Because of that, you may accidentally have many more parents in your population gene pool than intended. 




## Running Examples
there are sevral folders present in the repository please run the following the "settings.config" to load these folders


## Results
to these relevant links SuperMario showcasing is happening for level 1-1 and 4-1 wall showcasing

Mario beating 1-1:
https://drive.google.com/file/d/11guVlGnHsyZAaDHihgDpyrR3ojYU5PcP/view?usp=share_link
Mario learning to walljump:
https://drive.google.com/file/d/1UdnBKsxDbfXtUMpsLsQzf8JkfmpuSPSG/view?usp=share_link
