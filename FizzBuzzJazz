import java.util.ArrayList;
import java.util.HashMap;
import java.util.List;
import java.util.Map;

public class FizzBuzz {
  public static String BuildNumber(int num, Map<Integer, String> divisors) {
    String res = "";
    for(Integer i : divisors.keySet())
      if (num % i == 0)
        res += divisors.get(i);
    if(res.length() == 0)
      return Integer.toString(num);
    return res;
  }
  
  public static List<String> fizzBuzz(int n) {
    List<String> result = new ArrayList<>();
    Map<Integer, String> divisors = new HashMap<>();
    divisors.put(3, "Fizz");
    divisors.put(5, "Buzz");
    divisors.put(7, "Jazz");
    for (int i = 1; i <= n; ++i)
      result.add(BuildNumber(i, divisors));
    return result;
  }
  
  public static void main(String[] args) {
    int n = 20;
    List<String> result = fizzBuzz(n);
    for (String s : result) {
      System.out.print(s + " ");
    }
  }
}
