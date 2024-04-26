code để chạy với mẫu 540 + 558

funannotate predict -i scaffolds.filled_mask_540.fa -o  \
    --species "Oryza sativa" \
    --busco_seed_species rice --cpus 12 \
    --busco_db embryophyta \
    (ở bước này có thể có lỗi, check xem nó đưa ra bao nhiêu gen model)

funannotate predict -i scaffolds.filled_mask_543.fa -o predict_543_redundans_m2500_train20 \
    --species "Oryza sativa" \
    --busco_seed_species rice --cpus 12 \
    --busco_db embryophyta \
    --min_training_models x (x = gen model 

funannotate predict -i scaffolds.filled_mask_543.fa -o predict_543_redundans_m2500_train20 \
    --species "Oryza sativa" \
    --busco_seed_species rice --cpus 12 \
    --busco_db embryophyta \
    --min_training_models 20
