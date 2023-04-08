#include <bits/stdc++.h>
using namespace std;

struct TreeNode
{
    int val;
    TreeNode *left;
    TreeNode *right;
    TreeNode(int v)
    {
        val = v;
        left = right = NULL;
    }
};

class BeingZero
{
public:
void printvector(TreeNode*root,vector<int>&v)
    {
        if(root==NULL)
            return;
        printvector(root->left,v);
        v.push_back(root->val);
        printvector(root->right,v);
    }
    vector<int> inorderTraversal(TreeNode* root) {
        vector<int>v;
        printvector(root,v);
        return v;
    }
    bool isBST(TreeNode *root)
    {
        bool isBSTResult = false;
        // TODO: Just complete given function and
        // return true if the given tree is BST else return false
        // Input Reading and Output Printing is already taken care
        vector<int>v;
        v=inorderTraversal(root);
        vector<int>a;
        a=v;
        sort(a.begin(),a.end());
        if(v==a)
          isBSTResult=true;
        return isBSTResult;
    }
};
