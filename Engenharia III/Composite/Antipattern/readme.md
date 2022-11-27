     package antipattern;

    public class Pão {
	   public void buy() {
		  System.out.println("Comprando pão...");
    	}
    }
    
    
    
 <hr>   
 
      package antipattern;

      public class Leite {
	      public void buy() {
	    	System.out.println("Comprando leite...");
	   }
   }
    
  <hr>
  
     package antipattern;

     import java.util.ArrayList;
     import java.util.List;

     public class Carrinho {
     private List<Leite> leites = new ArrayList<Leite>();
	   private List<Pão> pães = new ArrayList<Pão>();
	
	   public void buy() {
	   	for(Leite can: leites)
		  {
		 	can.buy();
	    }
		   for(Pão cad: pães)
	   	{
			 cad.buy();
		    }
	    	System.out.println("Compra realizada!");
		     leites.clear();
		     pães.clear();
     	}

	    public void addLeite(Leite c){
	   	this.leites.add(c);
	    }
	
	    public void addPão(Pão c){
	   	this.pães.add(c);
	    }
	
	    public void removeLeite(Leite c){
	   	leites.remove(c);
     	}
	
	    public void removePão(Pão c){
		  pães.remove(c);
     	}
	
     }
