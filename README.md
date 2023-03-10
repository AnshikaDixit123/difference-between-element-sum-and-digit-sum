# difference-between-element-sum-and-digit-sumint sum_of_num = 0;
int sum1 = 0;
int sum2 =0;
int digit_sum = 0;
for(int i=0; i<nums.length; i++){
sum_of_num = sum_of_num + nums[i];
}
for(int i=0; i<nums.length; i++){
if(nums[i]<10){
sum1 = sum1 + nums[i];
}
else if(nums[i]>9){
while(nums[i]!=0){
sum2 = sum2 + nums[i]%10;
nums[i] = nums[i]/10;
}
}
}
digit_sum = sum1+sum2;
int ans = sum_of_num - digit_sum;
return ans;


        
    }
}
