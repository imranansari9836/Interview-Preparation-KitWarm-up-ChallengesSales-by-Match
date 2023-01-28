 public static int sockMerchant(int n, List<Integer> ar) {
    // Write your code here
    //10 20 20 10 10 30 50 10 20
    int count=0;
    HashSet<Integer>set=new HashSet<>();
    for(int i=0;i<ar.size();i++)
    {
        int element=ar.get(i);//
        if(set.contains(element))
        {
            set.remove(element);
            count++;//3
        }
        else{
            set.add(element);
        }
    }
    return count;

    }

}
