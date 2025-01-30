
'''
trialing using problem solving and logic to sort an Array - learnt it's somewhat a hybrid of bubble and selection sort
Thought I'd see what chatGPT would come up with and comapare results
'''
#MY CODE
#Lets get some runtime metrics
import time
start_time = time.time()

#ARRAY SORT
myArray = [1,10,5,11,17,8,3,7]

#get the first element of the array for comparison

#loop through all elements of the array 
def sweep():
    c = 0
    e = 0
    while c+1 < len(myArray):
        if myArray[e] > myArray[c+1]:
            val = myArray[e]
            myArray.pop(e)
            myArray.append(val)
            c+=1
        else:
            c+=1
            e+=1
        #print(myArray)
    return myArray

run = True
while run == True:
    if myArray == sorted(myArray):
        print(myArray)
        run = False
        print("--- %s seconds ---" % (time.time() - start_time))
    else:
        sweep()
 #END MY CODE       
 
#VS

#CHAT GPT 
# Start timer
start_time = time.time()

# Unsorted array
myArray = [1, 10, 5, 11, 17, 8, 3, 7]

# Hybrid Sort (Selection + Bubble)
def hybrid_sort(arr):
    n = len(arr)
    for i in range(n):
        max_idx = 0  # Track the index of the largest element
        for j in range(n - i):  # Reduce range as elements get sorted
            if arr[j] > arr[max_idx]:
                max_idx = j  # Update max index

        # Move the largest element to the end of the unsorted part
        arr.append(arr.pop(max_idx))  # Removes and appends to the end
        print(arr)  # Print the array after each step
       # time.sleep(0.3)  # Slow down for visualization

hybrid_sort(myArray)

# End timer
print("Sorted array:", myArray)
print("--- %s seconds ---" % (time.time() - start_time))
#END CHAT GPT

'''
After running my code had a runtime of 6ms to sort the array, chat gpt had a runtime of 10ms - Claiming that a victory for the humans a new sorting algorithm that beats the machine :P
'''


