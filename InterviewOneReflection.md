# Reflecting On My First Mock Interview

## Strengths
I think may biggest strength was answering the conceptual questions. I had no problem communicating what I knew about the four pillars of programming. I also was able to describe inheritance and the difference between interfaces and abstract classes.

## Weaknesses
I noticed two major weaknesses. As far as the technical part of the interview, I was unable to solve the problem and even talked about how I had a hard time grasping arrays. I absolutely have to fix that problem before the final round of interviews. I also noticed that I was looking at the screen straight on when answering questions so it looked like I wasn't very confident. I'll look right into the camera from now on. ## Technical Question Answer

## Technical Question Solution
Given an array nums, write a function to move all 0's to the end of it while maintaining the relative order of the non-zero elements.

You must do this in-place without making a copy of the array.
Minimize the total number of operations.

Example:

Input: [0,1,0,3,12]
Output: [1,3,12,0,0]

``` java
        public static void main(String[] args) {
            int[] ints = {0, 1, 0, 3, 12};
            orderArray(ints);
        }

        public static int[] orderArray(int[] nums){
            int temp;
            for(int i = 0; i < nums.length; i++) {
                for (int j = i + 1; j < nums.length; j++) {
                    if (nums[i] == 0) {
                        temp = nums[i];
                        nums[i] = nums[j];
                        nums[j] = temp;
                    }
                }
            }
            return nums;
        }
}
```
