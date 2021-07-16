The analysis code of the data can be found at https://github.com/LibiF

The data is organized in a table where each row corresponds to a recorded unit. 
Column legend:
rec_date - recording date (and penetration number) during which the unit was recorded
clus_num - id of the cluster assigned to it by Kilosort2. Note that this number is only unique whithin a single recording.
clus_depth - within brain depth of the cluster
clus_channel - channel from which the unit was recorded
acronym - acronym of the assinged brain region (AUDp=primary auditory cortex, AUDv=secondary/ventral auditory cortex, TEa/TeA= auditory Temporal Association cortex).
layer - cortical layer assigned to the unit
name - full name of the assigned brain region (of the acronym)
clus_classification - division to single units (SUs) = 2 and multi units (MUs) = 1
PT_raster - raster of pure tone responses comprised of 1440 rows and 700 columns. Each row is a trial and each column is a single milisecond. The trials are ordered by frequency and attenuation. 30 different frequencies were played in 4 sound attenuations such that each frequency x attenuation combination was played for 12 repetitions. Trials are ordered from lowest frequency to highest and within frequency are ordered from the loudest sound level to the most attenuated. Example - trials 1-12 3 kHz at 72 dB SPL, trials 13-24 3 kHz at 62 dB SPL, etc...
PT_PSTH - a mean over trials of the PT_raster.
log_responses - raster of responses to logarithimic FM_sweeps from most decreasing to most increasing. 10 logarithmic FMs were played such that 5 were decreasing and 5 were increasing in opposite slopes. Each FM was played for 12 repetitions in a single sound amplitude of 62 dB SPL. 
log_PSTH - mean responses to the 10 logarithmic FM sweeps ordered from the mean response to the most decreasing FM up to the most increasing FM.
