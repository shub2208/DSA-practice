// "static void main" must be defined in a public class.
public class Main {
   static int pivotBinarySearch(int[] arr , int  n , int  key){
       int pi = pivot(arr,0,n-1);
       if(pi == -1)
           return binarySearch(arr , 0,n-1,key);
       if(arr[pi] == key)
           return pi;
       if(arr[0]<= key)
          return binarySearch(arr,0,pi-1,key);
             return binarySearch(arr,pi+1,n-1,key);
   }
        static int pivot(int [] arr, int low, int high){
            if(high < low)
                return -1;
            if(high ==low)
                return low;
            int mid = low +(high-low)/2;
            if(mid < high && arr[mid] > arr[mid+1] )
                return mid;
             if(mid > low && arr[mid] < arr[mid-1] )
                return (mid-1);
            if (arr[low] >= arr[mid])
                return pivot(arr ,low, mid -1);
                return pivot(arr ,mid+1, high);            
        }
        static int binarySearch(int arr[] , int low , int high, int key){
            if(high < low )
                return -1;
            int mid = low +(high-low)/2;
            if (key == arr[mid])
                return mid;
            if (key > arr[mid])
                return binarySearch(arr , (mid+1), high, key);
            return binarySearch(arr , low, (mid-1), key);
            
    }
    public static void main(String[] args) {
        System.out.println("Hello World!");
        int [] arr ={5, 6, 7, 8, 9, 10, 1, 2, 3};
        int n = arr.length;
        int key = 9;
        System.out.println(pivotBinarySearch(arr ,n, key));
    }
}
