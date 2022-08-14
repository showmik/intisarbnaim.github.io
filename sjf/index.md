# Shortest Job First Scheduling (SJF)


Shortest Job First Scheduling (SJF)

<!--more-->

# Shortest Job First Scheduling (SJF)

## Non-Preemtive

```C
#include<stdio.h>
int main()
{
    int length;
    printf("Enter number of process: ");
    scanf("%d",&length);

    int p[length];
    float burstTime[length], waitingTime[length];

    // Input Burst Time
    for(int i=0; i<length; i++)
    {
        printf("Enter P%d Burst Time: ",i+1);
        scanf("%f", &burstTime[i]);
        p[i] = i+1;
    }

    //Sorting Burst Times
    for(int i=0; i<length; i++)
    {
        int pos = i;
        for(int j = i+1; j<length; j++)
        {
            if(burstTime[j] < burstTime[pos])
                pos = j;
        }

        float temp = burstTime[i];
        burstTime[i] = burstTime[pos];
        burstTime[pos] = temp;

        temp = p[i];
        p[i] = p[pos];
        p[pos] = temp;
    }

    // Calculating Waiting Times
    waitingTime[0] = 0;
    float total = 0;
    for(int i=1; i<length; i++)
    {
        waitingTime[i] = 0;
        for(int j=0; j<i; j++)
            waitingTime[i] += burstTime[j];

        total += waitingTime[i];
    }

    // Calculating Average Waiting Time
    float avgWaitingTime = (float)total / length;

    // Printing Results
    printf("\nProcess\t Burst Time\t Waiting Time");
    for(int i=0; i<length; i++)
    {
        printf("\nP%d\t  %.2f\t\t    %.2f", p[i], burstTime[i], waitingTime[i]);
    }
    printf("\n\nAverage Waiting Time=%.2f",avgWaitingTime);
}


```
### Output

<img src="/images/sjf_np_output.png"  alt="Output"/>
