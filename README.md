# HackerRankNotes
https://www.hackerrank.com/challenges/compare-the-triplets/problem?isFullScreen=true

 public static List<Integer> compareTriplets(List<Integer> a, List<Integer> b) { 
        
List<Integer> newArray = new ArrayList<>(Arrays.asList(0, 0));
      
        for(int i = 0; i< a.size();i++){
            
          if(a.get(i) > b.get(i)){
    newArray.set(0, newArray.get(0) + 1);
} else if(a.get(i) < b.get(i)){
    newArray.set(1, newArray.get(1) + 1); 
}

            
        }
        return newArray;
        

    }

}
