kinect-record-replay
====================

Sample code to record and replay kinect skeleton data based on Kinect Avateering project from Kinect SDK 1.8

```c#
private void Compare(Skeleton actSkel, Skeleton recSkel, GameTime gameTime)
        {
            actSkel = new Skeleton();
            recSkel = new Skeleton();
            
            for (int i = 0; i < jType.Count; i++)
            {
                double actX = actSkel.Joints[jType[i]].Position.X;
                double actY = actSkel.Joints[jType[i]].Position.Y;
                double actZ = actSkel.Joints[jType[i]].Position.Z;

                double recX = recSkel.Joints[jType[i]].Position.X;
                double recY = recSkel.Joints[jType[i]].Position.Y;
                double recZ = recSkel.Joints[jType[i]].Position.Z;
            }
           
        }
```
