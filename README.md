# Translation


Given:
Input embedding size (m)=256
Hidden state size (encoder + decoder) ( k )=256
Sequence length (input and output) ( T ) = 20(say)
Vocabulary size (source and target) ( V ) = 60(say)
Using 1-layer LSTM for both encoder and decoder
No attention
Inference is greedy decoding
Total computations = T×[8k(m+k)+kV]
substituting above values = 20×[8×256(256+256)+256×60]
                          =  21278720
Therefore, Total number of computation done by the network = 21.28 million operations

Total Parameters = 2Vm+8k(m+k+1)+kV+V
substituting above values = 2×60×256+8×256(256+256+1)+256×60+60
                          = 1100464
Therefore, total number of parameters in your network = 1.10 million parameters

