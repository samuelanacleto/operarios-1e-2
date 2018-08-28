public class Operario {
   String nome;
   float valorHora;
   float horasTrabalhadas;
   
   public void setNome(String nome){
	   this.nome=nome;
   }
   
   public String getNome(){
	   return this.nome;
   }
   
   public void setValorHora(float v){
	   this.valorHora=v;
   }
   
   public void setHorasTrabalhadas(float v){
	   this.horasTrabalhadas=v;
   }
   
   public float calcSalBruto(){
	   return this.horasTrabalhadas*this.valorHora;
   }
}
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\


public class Teste {

	public static void main(String[] args) {
		Operario op1 = new Operario();
		op1.setNome("João");
		op1.setHorasTrabalhadas(100);
		op1.setValorHora(20);
		
		Operario op2 = new Operario();
		op2.setNome("Maria");
		op2.setHorasTrabalhadas(80);
		op2.setValorHora(15);
		
		System.out.println(op1.calcSalBruto());
		System.out.println(op2.calcSalBruto());
	}
}
