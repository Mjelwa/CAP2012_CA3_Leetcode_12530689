class Solution {
public:
    void moveZeroes(vector<int>& nums) {
        int writeIdx = 0;

        for (int readIdx = 0; readIdx < static_cast<int>(nums.size()); ++readIdx) {
            if (nums[readIdx] != 0) {
                if (readIdx != writeIdx) {
                    swap(nums[readIdx], nums[writeIdx]);
                }
                ++writeIdx;
            }
        }
    }
};
