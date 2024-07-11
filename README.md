# Java-Networking-Programming
Develop ClientServer,GUI Chat and other apps


#getting ip from domain

import java.net.InetAddress;
import java.net.UnknownHostException;

public class main{
    public static void main(String[] args) throws UnknownHostException{
        InetAddress watcho=InetAddress.getByName("www.worthcrete.com");
        System.out.println(watcho);
    }  
    
}
output=>
www.worthcrete.com/104.21.84.192
=== Code Execution Successful ===
