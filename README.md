# Standard-Deviation-Calculator
Coded in Java


     import java.*;
    import java.lang.Math; 

    class Main {
    //assign variables
    static double standardDeviation = 0;
    static double mean = 0;

    static double data1 = 5;
    static double data2 = 8;
    static double data3 = 2;
    static double data4 = 11;

    public static void main (String[] args) {
      //call function
      mean = calcMean();
      standardDeviation = calcStandardDeviation();

      //print result
      System.out.println("Data 1: " + data1 + "     Data 2: " + data2 + "     Data 2: " + data3 + "     Data 4: " + data4);
      System.out.println("Mean= " + mean);
      System.out.println("Standard Deviation= " + standardDeviation);
    }

    public static double calcMean() {
      return ((data1+data2+data3+data4)/4);
    }

    public static double calcStandardDeviation() {
      return Math.sqrt(((data1 - mean)*(data1 - mean) + (data2 - mean)*(data2 - mean) + (data3 - mean)*(data3 - mean) + (data4 - mean)*(data4 - mean))/4);
    }
  }
