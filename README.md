# leedcode-119.-pascals-triangle-2
leedcode 119.pascals triangle 2 solution

class Solution {
    public List<Integer> getRow(int rowIndex) {
        List<Integer> list=new ArrayList<Integer>();
        long previous=1;
        list.add((int)previous);


       
        for(int i=1;i<=rowIndex;i++){
             long current=(previous*(rowIndex-i+1))/i;
             list.add((int) current);
             previous=current;    
            

        }
        return list;
    }
}
