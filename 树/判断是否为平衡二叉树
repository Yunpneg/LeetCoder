class Solution {
public:
    bool IsBalanced_Solution(TreeNode* pRoot) {
        if(pRoot == NULL)
            return true;
        int leftDepth = getDepth(pRoot -> left);
        int rightDepth = getDepth(pRoot -> right);
        if(leftDepth > rightDepth + 1 || leftDepth + 1 < rightDepth)
            return false;
        else
            return IsBalanced_Solution(pRoot -> left) && IsBalanced_Solution(pRoot -> right);
    }
     
    int getDepth(TreeNode* pRoot){
        if(pRoot == NULL)
            return 0;
        int leftDepth = getDepth(pRoot -> left);
        int rightDepth = getDepth(pRoot -> right);
        return leftDepth > rightDepth ? leftDepth + 1 : rightDepth + 1;
    }
};
