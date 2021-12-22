# Original LOLA-DICE

python3 lola_dice_original.py --logdir ./results/inner_128_outer128_baseline

python3 lola_dice_original.py --inner_exact --logdir ./results/inner_exact_outer128_baseline

python3 lola_dice_original.py --inner_batch_size 1024 --logdir ./results/inner1024_outer128_baseline

python3 lola_dice_original.py --inner_exact --outer_exact --logdir ./results/inner_exact_outer_exact

# LOLA-DICE Ablation study

python3 lola_dice_ablation.py --hessian_batch_size 1024 --logdir ./result_ablation/comp_128_hessian_1024

python3 lola_dice_ablation.py --hessian_exact --logdir --logdir ./result_ablation/comp_128_hessian_exact

python3 lola_dice_ablation.py --comp_exact --logdir ./result_ablation/comp_exact_hessian_128

python3 lola_dice_ablation.py --comp_batch_size 1024 --logdir ./result_ablation/comp1024_hessian_128

# LOLA-DICE Off-policy and ablation study
python3 lola_dice_off_policy.py --logdir ./result_offpolicy/off_policy

python3 lola_dice_off_policy_ablation.py --comp_on_policy --logdir ./result_offpolicy/off_comp_on_hessian

python3 lola_dice_off_policy_ablation.py --hessian_on_policy --logdir ./result_offpolicy/on_comp_off_hessian