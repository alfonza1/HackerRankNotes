# HackerRankNotes
https://www.hackerrank.com/challenges/compare-the-triplets/problem?isFullScreen=true


     public static List<Integer> compareTriplets(List<Integer> a, List<Integer> b) { 
 
     List<Integer> newArray = new ArrayList<>(Arrays.asList(0, 0));

      for(int i = 0; i< a.size();i++){
          if(a.get(i) > b.get(i)){
    newArray.set(0, newArray.get(0) + 1);
    }  
         else if(a.get(i) < b.get(i)){
        newArray.set(1, newArray.get(1) + 1);}
        }
     
        return newArray;
        
        }
      



https://hackerrank.com/challenges/plus-minus/problem?isFullScreen=true
    
    public static void plusMinus(List<Integer> arr) {
    // Initialize counters
    double positiveCount = 0;
    double negativeCount = 0;
    double zeroCount = 0;
    
    // Count positive, negative, and zero numbers
    for (int num : arr) {
        if (num > 0) {
            positiveCount++;
        } else if (num < 0) {
            negativeCount++;
        } else {
            zeroCount++;
        }
    }
    
    // Calculate and print the ratios
    System.out.println(String.format("%.6f", positiveCount / arr.size()));
    System.out.println(String.format("%.6f", negativeCount / arr.size()));
    System.out.println(String.format("%.6f", zeroCount / arr.size()));
}
