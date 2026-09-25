The results of the U2UT Model with 1000/250 data split trained in successive 6 stages are contained here:
Each stage contained different 1000 parallel audio samples of English and Yoruba.
Each stage used the same 250 validation samples.
Each 1000 train samples were chosen from the same pool.
Adam optimiser with lr set to 1e-4 was used, without a scheduler.
Loss was computed with cross entropy loss function without label smooting.
LSTM based phoneme decoder (target discrete) was used with 6 and 2 layers for encoder and decoder respectively. MHSA and MHCA were each set to 4,
d_model was set to 512, seq_len to 600, dropout was set to 0.1, feedfoward dimension was set to 1024.
