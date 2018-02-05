# DaysJudge
judge how many days a month in a special year.
package java_code;

public class DaysJudge {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int year=1900,month=2,days=0;
		switch(month){
		case 1:
		case 3:
		case 5:
		case 7:
		case 8:
		case 10:
		case 12:
			days=31;
			break;
		case 4:
		case 6:
		case 9:
		case 11:
			days=30;
			break;
		case 2:
			if((year%4==0)&&(year%100!=0)||(year%400)==0)
				days=29;
			else
				days=28;
			break;
		default:
			System.out.println("年月有误，请检查");
		
		}
		System.out.println(year+"年"+month+"月共有"+days+"天");

	}

}
