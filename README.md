# cell-balancing
# cell baklancing function block code

function [s1,s2,s3] = fcn(u1, u2, u3)

u1=int32(u1)
u2=int32(u2)
u3=int32(u3)

if((u1>u2) || (u1>u3))
    s1=1;
else
    s1=0;
end

if((u2>u1) || (u2>u3))
    s2=1;
else
    s2=0;
end
    if((u3>u1) || (u3>u2))
        s3=1;
    else
        s3=0;
    end

