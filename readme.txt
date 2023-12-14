D:\BoyangDeng\Prompt\CoOp\datasets
weed2021.py

bash scripts/cocoop/base2new_train.sh weed2021 1
bash scripts/cocoop/base2new_test.sh weed2021 1

bash scripts/coop/main.sh weed2021 rn50 end 16 16 False
bash scripts/coop/main.sh weed2021 rn50 end 16 16 True

How to initialize the context tokens with pre-trained word vectors? 
CTX_INIT: "a photo of a"

How to visualize nearest words for the learned context tokens?
python interpret_prompt.py D:\BoyangDeng\Prompt\CoOp\output\base2new\train_base_weed_6sku\weed2021\shots_16\CoCoOp\vit_b16_c4_ep10_batch1_ctxv1\seed1/prompt_learner/model.pth.tar 3