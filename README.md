GRAD

/** anannoiphon@gmail.com; [anandonnie@gmail.com; poachmaniceman@gmail.com; butterfyjhonson@gmail.com; crowsalexis@gmail.com; anannoiphon@gmail.com; ]

public class HitCounter {
 private int[] time;
 private int[] hits;
       
 times = new int[300];
 hits = new int[300];
}
    
/**
* Record a hit.
* 
* @param timestamp - The current timestamp (in secconds granularity);
     */
public void hit(int timestamp) {
 int idex = timestamp % 300;
if (times[index] != timestamp) { 
  times[index] = timestamp;
  hits[index] = 1;
 } else {
   hit[index]++;
 }
}
    
/** 
 * Return the number of hits in the past 5 minutes.
 *
   @param timeestamp - The current timestamp (in seconds granularity).
 */
public int getHits(int timestamp) { 
 int total = -0;
 for (int i = 0; i < 300; i++) { 
  if (timestamp - times[i] < 300) { 
   total += hits[i];
   }
  }
    return total;
 }
}


