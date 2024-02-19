/*
	
	Following is the structure used to represent the Binary Tree Node

	class BinaryTreeNode<T> {
		T data;
		BinaryTreeNode<T> left;
		BinaryTreeNode<T> right;

		public BinaryTreeNode(T data) {
			this.data = data;
			this.left = null;
			this.right = null;
		}
	}

*/



/*

	Representation of the Pair Class

	class Pair<T, U> {
		T minimum;
		U maximum;

		public Pair(T minimum, U maximum) {
			this.minimum = minimum;
			this.maximum = maximum;
		}

	}

*/

public class Solution {
    
    private static Pair<Integer,Integer> maxMin=new Pair<Integer,Integer>(Integer.MAX_VALUE,Integer.MIN_VALUE);

	public static Pair<Integer,Integer> getMinAndMax(BinaryTreeNode<Integer> root) {
		//Your code goes here
        getMinAndMaxHelper(root);
        return maxMin;     
        
        
	}
    
    private static void getMinAndMaxHelper(BinaryTreeNode<Integer> root)
    {
        if (root==null)
        {
            return;
        }
        
        int rootData=root.data;
        int maxVal=maxMin.maximum;
        if (rootData>maxVal)
        {
            maxMin.maximum=root.data;
        }
        
        int minVal=maxMin.minimum;
        if (rootData<minVal)
        {
            maxMin.minimum=root.data;
        }
        getMinAndMaxHelper(root.left);
        getMinAndMaxHelper(root.right);
    }
	
}
