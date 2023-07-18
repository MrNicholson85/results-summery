<template>
    <div class="result_sum">
        <div class="result_sum_container">
            <div class="result_sum_col_left">
                <div class="result_sum_heading">Your Results</div>
                <div class="result_sum_score">
                    <span class="result_sum_result">76</span>
                    <span class="result_sum_overall">of 100</span>
                </div>
                <div class="result_sum_message">Great</div>
                <div class="result_sum_copy">Your performance exceed 65% of the people conducting the test here!</div>
            </div>
            <div class="result_sum_col_right">
                <span class="result_sum_right_title">Summary</span>
                <ul class="pt-[24px] md:pt-[28px] grid gap-[16px] place-content-center">
                    <li class=" bg-red/5 result_sum_item">
                        <div class="flex justify-between">
                            <div class="flex gap-[12px] items-center">
                                <i class="pt-[4px]"><img :src="reactionIcon"/></i>
                                <span class="text-[18px] font-groteskmed text-red">Reaction</span>
                            </div>
                            <div class="flex gap-[12px] items-center">
                                <div class="result_sum_curr_val">80</div>
                                <div class="result_sum_full_val">/ 100</div>
                            </div>
                        </div>
                    </li>
                    <li class=" bg-yellow/5 result_sum_item">
                        <div class="flex justify-between">
                            <div class="flex gap-[12px] items-center">
                                <i class="pt-[4px]"><img :src="memeryIcon"/></i>
                                <span class="text-[18px] font-groteskmed text-yellow">Memery</span>
                            </div>
                            <div class="flex gap-[12px] items-center">
                                <div class="result_sum_curr_val">92</div>
                                <div class="result_sum_full_val">/ 100</div>
                            </div>
                        </div>
                    </li>
                    <li class=" bg-green/5 result_sum_item">
                        <div class="flex justify-between">
                            <div class="flex gap-[12px] items-center">
                                <i class="pt-[4px]"><img :src="verbalIcon"/></i>
                                <span class="text-[18px] font-groteskmed text-green">Verbal</span>
                            </div>
                            <div class="flex gap-[12px] items-center">
                                <div class="result_sum_curr_val">61</div>
                                <div class="result_sum_full_val">/ 100</div>
                            </div>
                        </div>
                    </li>
                    <li class=" bg-blue/5 result_sum_item">
                        <div class="flex justify-between">
                            <div class="flex gap-[12px] items-center">
                                <i class="pt-[4px]"><img :src="visualIcon"/></i>
                                <span class="text-[18px] font-groteskmed text-blue">Visual</span>
                            </div>
                            <div class="flex gap-[12px] items-center">
                                <div class="result_sum_curr_val">73</div>
                                <div class="result_sum_full_val">/ 100</div>
                            </div>
                        </div>
                    </li>
                </ul>
                <button class="result_sum_btn hover:bg-gradient-to-b  from-g-purpl-1 to-g-purple-2">
                    Continue
                </button>
            </div>
        </div>
    </div>
</template>

<script setup>
import reactionIcon from '../assets/images/icon-reaction.svg';
import memeryIcon from '../assets/images/icon-memory.svg';
import verbalIcon from '../assets/images/icon-verbal.svg';
import visualIcon from '../assets/images/icon-visual.svg';

</script>

<style scoped>
.result_sum {
    @apply bg-[#ECF2FF] absolute w-full h-full
}

.result_sum_container {
    @apply w-[375px] md:w-[736px] m-auto grid md:flex md:rounded-[32px] bg-super-white md:shadow-[0px_30px_60px_0px_rgba(61,108,236,0.15)] md:top-[50%] md:-translate-y-[50%] md:relative
}

.result_sum_col_left {
    @apply  md:w-[368px] bg-gradient-to-b  from-g-purpl-1 to-g-purple-2 md:rounded-tl-[32px] md:rounded-tr-[32px] rounded-bl-[32px] rounded-br-[32px] grid justify-center px-8 pt-[24px] md:pt-[38px] pb-[55px] h-[356px] md:h-[512px]
}

.result_sum_heading {
    @apply text-light-blue font-groteskbold text-center text-[18px] md:text-[24px]
}

.result_sum_score {
    @apply w-[140px] h-[140px] md:w-[200px] md:h-[200px] mt-[15px] md:mt-[35px] rounded-[50%] bg-gradient-to-b from-g-dark-purpl-1 m-auto grid items-center text-center place-content-center
}

.result_sum_item {
    @apply grid items-center w-[315px] md:w-[288px] h-[56px] rounded-[12px] px-[18px]
}

.result_sum_result {
    @apply text-super-white font-groteskextrabold text-[56px] md:text-[72px] leading-[72px]
}

.result_sum_overall {
    @apply text-[18px] font-groteskbold text-light-blue
}

.result_sum_message {
    @apply text-center pt-[28px] text-super-white font-groteskbold text-[24px] md:text-[32px]
}

.result_sum_copy {
    @apply text-center text-light-blue font-groteskmed text-[16px] md:text-[18px] w-[260px] m-auto pt-[5px]
}

.result_sum_col_right {
    @apply px-[30px] md:px-[40px] pt-[24px] md:pt-[38px] h-[462px] md:h-[512px]
}
.result_sum_right_title{
    @apply text-[18px] md:text-[24px] font-groteskbold text-dark-navy
}

.result_sum_btn {
    @apply text-super-white text-[18px] w-full rounded-[128px] bg-dark-navy py-[17px] mt-[24px] md:mt-[41px]
}



.result_sum_full_val {
    @apply text-[16px] leading-[16px] md:leading-[18px] md:text-[18px] text-dark-navy/50 font-groteskbold
}

.result_sum_curr_val {
    @apply text-[16px] leading-[16px] md:leading-[18px] md:text-[18px] text-dark-navy font-groteskbold
}
</style>