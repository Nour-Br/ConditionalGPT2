# ConditionalGPT2

## DataSets 
copy your data from your directory to snips folder
```cd  /ConditionalGPT2/src/utils/
cp  YourDir/test.in /ConditionalGPT2/test.seq
cp  YourDir/testLabel.in /ConditionalGPT2/test.label
paste -d'\t'  test.label  test.seq > test.tsv
```
repeat these for train and valid data

## Dependencies 
To run this code, you need following dependencies 
- Pytorch 1.5
- fairseq 0.9 
- transformers 2.9 

## How to run 
```python /ConditionalGPT2/src/bert_aug/cgpt2.py \
         --data_dir '/ConditionalGPT2/src/utils/datasets/snips' \
         --output_dir '/ConditionalGPT2/cgpt2' \
         --num_train_epochs 10 \
         --block_size 64 \
         --learning_rate 5e-05 \
```
## License

This project is licensed under the Creative Common Attribution Non-Commercial 4.0 license.

   


