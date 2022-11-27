      package antipattern;
      
      Analógico.java

      public class Analógico implements Cronômetro{

    	public void update(int state) {
	   	System.out.println("Analógico: " + Integer.toString(state));		
	     }

     }

<hr>

    Digital.java

     package antipattern;

    public class Digital implements Cronômetro  {

	   public void update(int state) {
	  	System.out.println("Digital: " + Integer.toString(state * 2));		
	   }
	
     }

<hr>

  

