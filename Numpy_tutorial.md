#### import numpy as np 
arr=np.array([1,2]) => `create ndarray`

np.__version__ => `version of numpy`

type(arr) =>  `the type of the object`

arr=np.array([[],[],[]]) =>  `2d array`

np.array(arr.ndim) =>  `dimension of array`

np.array(arr,ndmin=x) => `redefine array as x dim`

print(arr[x,y]) =>  `access element in array`

print(arr[start,end,step]) => `access interval in array, end not include`


print(x,dtype) => `return type of x`

arr=np.array([1,2],dtype='x') => `create array with type x`

arr2=arr.astype('i') => `convert type of arr to 'i'`

new=x.copy() => `create copy from x`

s=x.view() => `view x as s which affected to any change in x,<br/>
                        any change in s will affect in x`
		
print(s.base) => `if s is copy => None. if view => return original array`

print(s.shape) => `the dimenson of element`

y=x.reshape(2,4) => `resize x to be 2d as y as view`

y=x.reshape(-1) => `convert to 1d`

for x in np.nditer(arr,flags=['buffered'] => `to free space for data` , op_dtype=['S']):<br/>
        print(x) => `print every value in arr whatever its dimension wih type S`
	
for i, x in np.mdenumerate(arr):<br/>
        print(i,x) 	=> `return x and its index location`
	
x=np.concatenate `or` stack ((arr1,arr2),axis=0 `or` 1)  => `concate arrays in line (1) or vertical (0)`

x=np.hstack((arr1,arr2)) => `concate to 1d line row [[] []] `

x=np.vstack((arr1,arr2)) => `concate to 1d line column  [[],[]]`

x=np.dstack((arr1,arr2)) => `concate to 1d line vertical in largest dimension [[1 4],[2 5],[3 6]]`

np.array_split(arr,4,axis=1) => `split arr to 4 arrays` , `also hsplit, vsplit, dsplit`

i=np.where(arr=x) => `return index of x`

y=np.sort(arr) => `sort arr`

n=y>6 =>  `boolean list`

m=y[N] => `numbers of index of true`
