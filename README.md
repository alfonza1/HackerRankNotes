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


https://www.hackerrank.com/challenges/staircase/problem?isFullScreen=true
   
     public static void staircase(int n) {
    for (int i = 1; i <= n; i++) {  // Iterate over row numbers
        for (int j = 0; j < n - i; j++) {  // Print spaces for the current row
            System.out.print(" ");
        }
        for (int j = 0; j < i; j++) {  // Print '#' characters for the current row
            System.out.print("#");
        }
        
        System.out.println();  // Newline after each row
    }
     }
     

https://www.hackerrank.com/challenges/array-left-rotation/problem?isFullScreen=true
          
     public static List<Integer> rotateLeft(int d, List<Integer> arr) {
        
        if(d > 0){
            for(int i = 0;i < d;i++){
               
                int front = arr.get(0);
                     
                for(int j =1;j < arr.size();j++ ){
                    
                    arr.set(j - 1,arr.get(j));
                }
                          arr.set(arr.size() - 1, front);
              }
        }
                      return arr;

    }







     
