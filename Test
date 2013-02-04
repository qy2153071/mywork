package com.resources;

import javax.servlet.http.HttpServletRequest;
import javax.ws.rs.GET;
import javax.ws.rs.Path;
import javax.ws.rs.PathParam;
import javax.ws.rs.Produces;
import javax.ws.rs.core.Context;
import javax.ws.rs.core.MediaType;

import org.codehaus.jettison.json.JSONException;
import org.codehaus.jettison.json.JSONObject;
  

@Path("/hello")  
public class HelloResource {  
    @GET  
    @Produces(MediaType.APPLICATION_JSON)  
    public String sayHello(@Context HttpServletRequest request) throws JSONException {  
      String callback = request.getParameter("callback");
    	JSONObject json = new JSONObject();
    	json.accumulate("user", "Hello Jersey");
    	if ("2" == "12") {
        	System.out.println(123);
        }
        return callback + "(" + json + ")";  
    }  
}    
