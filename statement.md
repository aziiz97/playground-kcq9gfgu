import java.util.ArrayList;
import java.util.Collections;
import java.util.List;
public class Main {  
    public static void main(String[] args) {
   List<Integer> data=new ArrayList<Integer>(){{
			add(-8);
			add(42);
			add(18);
			add(0);
			add(-16);
		}};
		List<Integer> res=new ArrayList<Integer>(data);
		int n=data.size();
		Collections.sort(res);
		for (int i = n - 2; i >= 0; --i)
			res.add(res.get(i));
		for (Integer element : data) 			
			System.out.print(element+" ");
		System.out.println("\n resultat :");
		for (Integer element : res) 			
			System.out.print(element+" ");;

    }
}

 

